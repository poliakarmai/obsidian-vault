---
title: "GSC Audit: /tmp/gsc_scan_targets/sshpiper"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/sshpiper

**Дата:** 29.06.2026 14:21  
**Путь:** `/tmp/gsc_scan_targets/sshpiper`  
**Всего находок:** 373  
**CRITICAL:** 3 | **HIGH:** 338 | **MEDIUM:** 28 | **LOW:** 3

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Go: Unhandled error | 156 |
| Хардкод IP адреса | 107 |
| Go: Goroutine leak | 39 |
| Go: sync.Mutex copy | 24 |
| Go: Hardcoded secret | 20 |
| Go: panic in library code | 9 |
| GS002 | 5 |
| GS003 | 3 |
| Go: println in production | 2 |
| Hardcoded encryption key | 2 |
| Go: crypto/md5 or crypto/sha1 | 1 |
| Go: math/rand for security | 1 |
| World-readable file: .goreleaser.yaml (664) | 1 |
| World-readable file: .devcontainer.json (664) | 1 |
| GS009 | 1 |
| GS014 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | e2eentry.sh | 85 | Match:                     base_key = "baseline:" name |
| CRITICAL | ? | e2eentry.sh | 86 | Match:                     piper_key = "sshpiper:" name |
| CRITICAL | ? | daemon.go | 326 | Match: 			hash := fmt.Sprintf("%x", md5.Sum([]byte(banner))) |
| HIGH | ? | pluginbase.go | 338 | Variable assignment ignoring error return value |
| HIGH | ? | util.go | 57 | Variable assignment ignoring error return value |
| HIGH | ? | skel_test.go | 172 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 76 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 106 | Variable assignment ignoring error return value |
| HIGH | ? | service_test.go | 188 | Variable assignment ignoring error return value |
| HIGH | ? | messagestream_test.go | 161 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 137 | Variable assignment ignoring error return value |
| HIGH | ? | dockersshd_bridge.go | 88 | Variable assignment ignoring error return value |
| HIGH | ? | dockersshd_bridge.go | 208 | Variable assignment ignoring error return value |
| HIGH | ? | dockersshd_bridge.go | 214 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 136 | Variable assignment ignoring error return value |
| HIGH | ? | docker.go | 63 | Variable assignment ignoring error return value |
| HIGH | ? | docker.go | 113 | Variable assignment ignoring error return value |
| HIGH | ? | docker.go | 139 | Variable assignment ignoring error return value |
| HIGH | ? | dockersshd_bridge_test.go | 78 | Variable assignment ignoring error return value |
| HIGH | ? | dockersshd_bridge_test.go | 155 | Variable assignment ignoring error return value |
| HIGH | ? | dockersshd_bridge_test.go | 158 | Variable assignment ignoring error return value |
| HIGH | ? | dockersshd_bridge_test.go | 161 | Variable assignment ignoring error return value |
| HIGH | ? | workingdir_test.go | 39 | Variable assignment ignoring error return value |
| HIGH | ? | lua_test.go | 589 | Variable assignment ignoring error return value |
| HIGH | ? | lua_test.go | 697 | Variable assignment ignoring error return value |
| HIGH | ? | lua_test.go | 700 | Variable assignment ignoring error return value |
| HIGH | ? | lua.go | 84 | Variable assignment ignoring error return value |
| HIGH | ? | lua.go | 727 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 52 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 194 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 195 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 216 | Variable assignment ignoring error return value |
| HIGH | ? | yaml.go | 125 | Variable assignment ignoring error return value |
| HIGH | ? | yaml.go | 157 | Variable assignment ignoring error return value |
| HIGH | ? | admin_test.go | 90 | Variable assignment ignoring error return value |
| HIGH | ? | admin_test.go | 120 | Variable assignment ignoring error return value |
| HIGH | ? | admin_test.go | 240 | Variable assignment ignoring error return value |
| HIGH | ? | admin_test.go | 251 | Variable assignment ignoring error return value |
| HIGH | ? | kubernetes_test.go | 47 | Variable assignment ignoring error return value |
| HIGH | ? | kubernetes_test.go | 117 | Variable assignment ignoring error return value |
| HIGH | ? | factory.go | 45 | Variable assignment ignoring error return value |
| HIGH | ? | factory.go | 101 | Variable assignment ignoring error return value |
| HIGH | ? | factory.go | 116 | Variable assignment ignoring error return value |
| HIGH | ? | factory.go | 147 | Variable assignment ignoring error return value |
| HIGH | ? | factory.go | 156 | Variable assignment ignoring error return value |
| HIGH | ? | factory.go | 169 | Variable assignment ignoring error return value |
| HIGH | ? | factory.go | 174 | Variable assignment ignoring error return value |
| HIGH | ? | main_test.go | 178 | Variable assignment ignoring error return value |
| HIGH | ? | fixed_test.go | 35 | Variable assignment ignoring error return value |
| HIGH | ? | clientset_generated.go | 26 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 63 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 78 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 379 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 457 | Variable assignment ignoring error return value |
| HIGH | ? | daemon_test.go | 294 | Variable assignment ignoring error return value |
| HIGH | ? | asciicast.go | 67 | Variable assignment ignoring error return value |
| HIGH | ? | asciicast.go | 106 | Variable assignment ignoring error return value |
| HIGH | ? | asciicast.go | 154 | Variable assignment ignoring error return value |
| HIGH | ? | envinject.go | 59 | Variable assignment ignoring error return value |
| HIGH | ? | zz_generated.deepcopy.go | 62 | Variable assignment ignoring error return value |
| HIGH | ? | zz_generated.deepcopy.go | 93 | Variable assignment ignoring error return value |
| HIGH | ? | envinject_e2e_test.go | 129 | Variable assignment ignoring error return value |
| HIGH | ? | kubernetes_test.go | 359 | Variable assignment ignoring error return value |
| HIGH | ? | kubernetes_test.go | 362 | Variable assignment ignoring error return value |
| HIGH | ? | daemon.go | 96 | Variable assignment ignoring error return value |
| HIGH | ? | daemon.go | 224 | Variable assignment ignoring error return value |
| HIGH | ? | daemon.go | 284 | Variable assignment ignoring error return value |
| HIGH | ? | daemon.go | 375 | Variable assignment ignoring error return value |
| HIGH | ? | daemon.go | 528 | Variable assignment ignoring error return value |
| HIGH | ? | daemon.go | 532 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 61 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 164 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 194 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 231 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 241 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 263 | Variable assignment ignoring error return value |
| HIGH | ? | skel.go | 308 | Variable assignment ignoring error return value |
| HIGH | ? | hook.go | 23 | Variable assignment ignoring error return value |
| HIGH | ? | kubectl_exec_bridge.go | 158 | Variable assignment ignoring error return value |
| HIGH | ? | kubectl_exec_bridge.go | 168 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 22 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 61 | Variable assignment ignoring error return value |
| HIGH | ? | server.go | 71 | Variable assignment ignoring error return value |
| HIGH | ? | server.go | 113 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 41 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 45 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 47 | Variable assignment ignoring error return value |
| HIGH | ? | streamhook.go | 83 | Variable assignment ignoring error return value |
| HIGH | ? | streamhook.go | 148 | Variable assignment ignoring error return value |
| HIGH | ? | streamhook.go | 162 | Variable assignment ignoring error return value |
| HIGH | ? | streamhook.go | 168 | Variable assignment ignoring error return value |
| HIGH | ? | streamhook.go | 174 | Variable assignment ignoring error return value |
| HIGH | ? | broadcaster.go | 63 | Variable assignment ignoring error return value |
| HIGH | ? | broadcaster.go | 85 | Variable assignment ignoring error return value |
| HIGH | ? | broadcaster.go | 104 | Variable assignment ignoring error return value |
| HIGH | ? | envinject_test.go | 32 | Variable assignment ignoring error return value |
| HIGH | ? | envinject_test.go | 49 | Variable assignment ignoring error return value |
| HIGH | ? | envinject_test.go | 62 | Variable assignment ignoring error return value |
| HIGH | ? | envinject_test.go | 90 | Variable assignment ignoring error return value |
| HIGH | ? | registry_test.go | 67 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 34 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 153 | Variable assignment ignoring error return value |
| HIGH | ? | registry.go | 77 | Variable assignment ignoring error return value |
| HIGH | ? | registry.go | 94 | Variable assignment ignoring error return value |
| HIGH | ? | registry.go | 111 | Variable assignment ignoring error return value |
| HIGH | ? | registry.go | 124 | Variable assignment ignoring error return value |
| HIGH | ? | broadcaster_test.go | 20 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 62 | Variable assignment ignoring error return value |
| HIGH | ? | httpapi.go | 83 | Variable assignment ignoring error return value |
| HIGH | ? | httpapi.go | 190 | Variable assignment ignoring error return value |
| HIGH | ? | httpapi.go | 204 | Variable assignment ignoring error return value |
| HIGH | ? | grpc.go | 74 | Variable assignment ignoring error return value |
| HIGH | ? | grpc.go | 233 | Variable assignment ignoring error return value |
| HIGH | ? | grpc.go | 247 | Variable assignment ignoring error return value |
| HIGH | ? | grpc.go | 261 | Variable assignment ignoring error return value |
| HIGH | ? | grpc.go | 295 | Variable assignment ignoring error return value |
| HIGH | ? | grpc.go | 692 | Variable assignment ignoring error return value |
| HIGH | ? | httpapi_test.go | 132 | Variable assignment ignoring error return value |
| HIGH | ? | chain.go | 39 | Variable assignment ignoring error return value |
| HIGH | ? | chain.go | 74 | Variable assignment ignoring error return value |
| HIGH | ? | chain.go | 157 | Variable assignment ignoring error return value |
| HIGH | ? | chain.go | 174 | Variable assignment ignoring error return value |
| HIGH | ? | chain.go | 182 | Variable assignment ignoring error return value |
| HIGH | ? | chain.go | 190 | Variable assignment ignoring error return value |
| HIGH | ? | loglevel_test.go | 30 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator_test.go | 80 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator_test.go | 145 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator_test.go | 152 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 39 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 199 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 230 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 236 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 256 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 285 | Variable assignment ignoring error return value |
| HIGH | ? | main.go | 290 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 74 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 96 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 102 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 103 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 112 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 113 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 135 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 165 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 169 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 170 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 184 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 198 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 209 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 227 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 238 | Variable assignment ignoring error return value |
| HIGH | ? | aggregator.go | 250 | Variable assignment ignoring error return value |
| HIGH | ? | ssh_server.go | 259 | Variable assignment ignoring error return value |
| HIGH | ? | ssh_server.go | 512 | Variable assignment ignoring error return value |
| HIGH | ? | ssh_server.go | 534 | Variable assignment ignoring error return value |
| HIGH | ? | ssh_server.go | 547 | Variable assignment ignoring error return value |
| HIGH | ? | ssh_server.go | 562 | Variable assignment ignoring error return value |
| HIGH | ? | ssh_server_test.go | 38 | Variable assignment ignoring error return value |
| HIGH | ? | ssh_server_test.go | 70 | Variable assignment ignoring error return value |
| HIGH | ? | ssh_server_test.go | 126 | Variable assignment ignoring error return value |
| HIGH | ? | grpcplugin_test.go | 27 | panic should only be used in init/main, return errors instea |
| HIGH | ? | grpcplugin_test.go | 40 | panic should only be used in init/main, return errors instea |
| HIGH | ? | grpcplugin_test.go | 105 | panic should only be used in init/main, return errors instea |
| HIGH | ? | clientset.go | 92 | panic should only be used in init/main, return errors instea |
| HIGH | ? | sshpiper_client.go | 61 | panic should only be used in init/main, return errors instea |
| HIGH | ? | asciicast.go | 21 | panic should only be used in init/main, return errors instea |
| HIGH | ? | clientset_generated.go | 28 | panic should only be used in init/main, return errors instea |
| HIGH | ? | grpc.go | 219 | panic should only be used in init/main, return errors instea |
| HIGH | ? | grpc.go | 673 | panic should only be used in init/main, return errors instea |
| HIGH | ? | skel_test.go | 265 | Match: 	host := "[127.0.0.1]:22" |
| HIGH | ? | lua_test.go | 75 | Match: 		remoteAddr: "192.168.1.100", |
| HIGH | ? | lua_test.go | 132 | Match: 		remoteAddr: "192.168.1.100", |
| HIGH | ? | lua_test.go | 152 | Match: 		remoteAddr: "192.168.1.101", |
| HIGH | ? | lua_test.go | 172 | Match: 		remoteAddr: "192.168.1.102", |
| HIGH | ? | lua_test.go | 219 | Match: 		remoteAddr: "192.168.1.100", |
| HIGH | ? | lua_test.go | 264 | Match: 				remoteAddr: "192.168.1.100", |
| HIGH | ? | lua_test.go | 365 | Match: 		remoteAddr: "192.168.1.100", |
| HIGH | ? | lua_test.go | 371 | Match: 		remoteAddr: "192.168.1.101", |
| HIGH | ? | lua_test.go | 523 | Match: 		remoteAddr: "192.168.1.100", |
| HIGH | ? | lua_test.go | 626 | Match: 	conn := &mockConnMetadata{username: "alice", remoteA |
| HIGH | ? | benchmark_test.go | 82 | Match: 			if err := runScpTransfer(b, "127.0.0.1", piperport |
| HIGH | ? | benchmark_test.go | 95 | Match: 			if err := runSSHStream(b, "127.0.0.1", piperport,  |
| HIGH | ? | lua_test.go | 179 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 210 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 241 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 272 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 309 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 364 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 401 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 464 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 558 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 623 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 688 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 749 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 814 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 877 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 938 | Match: 			"127.0.0.1", |
| HIGH | ? | lua_test.go | 1006 | Match: 			"127.0.0.1", |
| HIGH | ? | workingdir_test.go | 87 | Match: 				"127.0.0.1", |
| HIGH | ? | workingdir_test.go | 209 | Match: 				"127.0.0.1", |
| HIGH | ? | admin_test.go | 31 | Match: 	adminAddr := "127.0.0.1:" + adminPort |
| HIGH | ? | admin_test.go | 35 | Match: 		"--admin-grpc-address", "127.0.0.1", |
| HIGH | ? | admin_test.go | 102 | Match: 		"127.0.0.1", |
| HIGH | ? | admin_test.go | 140 | Match: 	if !strings.Contains(live.GetDownstreamAddr(), "127. |
| HIGH | ? | admin_test.go | 141 | Match: 		t.Errorf("Session.DownstreamAddr = %q, want it to c |
| HIGH | ? | admin_test.go | 279 | Match: 		"--admin-grpc-address", "127.0.0.1", |
| HIGH | ? | no_penalties.conf | 1 | Match: PerSourcePenaltyExemptList 0.0.0.0/0 |
| HIGH | ? | yaml_test.go | 267 | Match: 			"127.0.0.1", |
| HIGH | ? | yaml_test.go | 299 | Match: 			"127.0.0.1", |
| HIGH | ? | yaml_test.go | 329 | Match: 			"127.0.0.1", |
| HIGH | ? | yaml_test.go | 360 | Match: 			"127.0.0.1", |
| HIGH | ? | yaml_test.go | 393 | Match: 			"127.0.0.1", |
| HIGH | ? | yaml_test.go | 424 | Match: 			"127.0.0.1", |
| HIGH | ? | yaml_test.go | 474 | Match: 			"127.0.0.1", |
| HIGH | ? | yaml_test.go | 507 | Match: 			"127.0.0.1", |
| HIGH | ? | yaml_test.go | 538 | Match: 			"127.0.0.1", |
| HIGH | ? | yaml_test.go | 567 | Match: 			"127.0.0.1", |
| HIGH | ? | docker-compose.yml | 104 | Match:         kubectl port-forward service/sshpiper --pod-r |
| HIGH | ? | docker-compose.yml | 120 | Match:       - SSHPIPERD_ALLOWED_PROXY_ADDRESSES=0.0.0.0/0 |
| HIGH | ? | grpcplugin_test.go | 25 | Match: 	l, err := net.Listen("tcp", "0.0.0.0:0") |
| HIGH | ? | grpcplugin_test.go | 103 | Match: 	l, err := net.Listen("tcp", "0.0.0.0:0") |
| HIGH | ? | main_test.go | 166 | Match: 	return net.JoinHostPort("127.0.0.1", (port)), port |
| HIGH | ? | failtoban_test.go | 50 | Match: 			"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 74 | Match: 			"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 87 | Match: 		if !strings.Contains(string(s), "Connection closed  |
| HIGH | ? | failtoban_test.go | 161 | Match: 			"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 191 | Match: 				"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 215 | Match: 			"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 229 | Match: 		if !strings.Contains(string(s), "Connection closed  |
| HIGH | ? | failtoban_test.go | 249 | Match: 		"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 274 | Match: 			"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 303 | Match: 			"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 331 | Match: 			"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 362 | Match: 		"127.0.0.1/8", |
| HIGH | ? | failtoban_test.go | 387 | Match: 			"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 416 | Match: 			"127.0.0.1", |
| HIGH | ? | failtoban_test.go | 444 | Match: 			"127.0.0.1", |
| HIGH | ? | connmeta_test.go | 45 | Match: 		"127.0.0.1", |
| HIGH | ? | fixed_test.go | 65 | Match: 				"127.0.0.1", |
| HIGH | ? | fixed_test.go | 112 | Match: 		"127.0.0.1", |
| HIGH | ? | fixed_test.go | 144 | Match: 		ValidPrincipals: []string{"127.0.0.1", "localhost"} |
| HIGH | ? | fixed_test.go | 186 | Match: 		"127.0.0.1", |
| HIGH | ? | stdout_test.go | 47 | Match: 		"127.0.0.1", |
| HIGH | ? | docker_test.go | 44 | Match: 			"127.0.0.1", |
| HIGH | ? | docker_test.go | 92 | Match: 			"127.0.0.1", |
| HIGH | ? | docker_test.go | 134 | Match: 			"127.0.0.1", |
| HIGH | ? | banner_test.go | 43 | Match: 			"127.0.0.1", |
| HIGH | ? | banner_test.go | 101 | Match: 			"127.0.0.1", |
| HIGH | ? | banner_test.go | 141 | Match: 				"127.0.0.1", |
| HIGH | ? | main.go | 127 | Match: 				Value:   "0.0.0.0", |
| HIGH | ? | main.go | 276 | Match: 				Value:   "127.0.0.1", |
| HIGH | ? | kubectl_exec_bridge.go | 85 | Match: 	listener, err := net.Listen("tcp", "127.0.0.1:0") |
| HIGH | ? | envinject_e2e_test.go | 30 | Match: 	upstreamLn, err := net.Listen("tcp", "127.0.0.1:0") |
| HIGH | ? | envinject_e2e_test.go | 38 | Match: 	piperLn, err := net.Listen("tcp", "127.0.0.1:0") |
| HIGH | ? | dockersshd_bridge.go | 35 | Match: 	listener, err := net.Listen("tcp", "127.0.0.1:0") |
| HIGH | ? | server_test.go | 18 | Match: 	srv := NewServer(reg, "test-id", "test-version", "12 |
| HIGH | ? | server_test.go | 22 | Match: 	lis, err := net.Listen("tcp", "127.0.0.1:0") |
| HIGH | ? | grpc.go | 651 | Match: 	conn, err := grpc.NewClient("127.0.0.1", grpc.WithTr |
| HIGH | ? | grpc_test.go | 51 | Match: 	if err := cb("host:22", mockAddr("1.2.3.4:22"), newT |
| HIGH | ? | grpc_test.go | 58 | Match: 	host := "[127.0.0.1]:2222" |
| HIGH | ? | grpc_test.go | 64 | Match: 	addr, err := net.ResolveTCPAddr("tcp", "127.0.0.1:22 |
| HIGH | ? | grpc_test.go | 76 | Match: 	host := "[127.0.0.1]:2222" |
| HIGH | ? | grpc_test.go | 82 | Match: 	addr, err := net.ResolveTCPAddr("tcp", "127.0.0.1:22 |
| HIGH | ? | grpc_test.go | 94 | Match: 	err := cb("host:22", mockAddr("1.2.3.4:22"), newTest |
| HIGH | ? | grpc_test.go | 110 | Match: 	if err := cb("host", mockAddr("1.2.3.4:22"), pub); e |
| HIGH | ? | grpc_test.go | 113 | Match: 	if mock.lastReq == nil || mock.lastReq.Hostname != " |
| HIGH | ? | grpc_test.go | 130 | Match: 	if err := cb("host", mockAddr("1.2.3.4:22"), newTest |
| HIGH | ? | grpc_test.go | 145 | Match: 	if err := cb("host", mockAddr("1.2.3.4:22"), newTest |
| HIGH | ? | grpc_test.go | 162 | Match: 	if err := cb("host", mockAddr("1.2.3.4:22"), newTest |
| HIGH | ? | ssh_server_test.go | 140 | Match: 	content := `from="10.0.0.0/8",command="echo hi" ` +  |
| HIGH | ? | ssh_server_test.go | 196 | Match: 			"--sshpiperd", "127.0.0.1:8082", |
| HIGH | ? | ssh_server_test.go | 208 | Match: 		"--sshpiperd", "127.0.0.1:8082", |
| HIGH | ? | aggregator_test.go | 39 | Match: 	lis, err := net.Listen("tcp", "127.0.0.1:0") |
| HIGH | ? | main.go | 54 | Match: 				Value:   "127.0.0.1", |
| HIGH | ? | httpapi_test.go | 44 | Match: 	lis, err := net.Listen("tcp", "127.0.0.1:0") |
| HIGH | ? | index.html | 58 | Match:       <path d="M12 .5C5.65.5.5 5.65.5 12a11.5 11.5 0  |
| HIGH | ? | plugin.pb.go | 81 | Match: 	Metadata      map[string]string      `protobuf:"byte |
| HIGH | ? | plugin.pb.go | 172 | Match: 	Env map[string]string `protobuf:"bytes,7,rep,name=en |
| HIGH | ? | plugin.pb.go | 547 | Match: 	Meta          map[string]string      `protobuf:"byte |
| HIGH | ? | plugin.pb.go | 591 | Match: 	Meta          map[string]string      `protobuf:"byte |
| HIGH | ? | lua_test.go | 26 | Match:             password = "pass", |
| HIGH | ? | lua_test.go | 71 | Match:             password = "pass", |
| HIGH | ? | lua_test.go | 90 | Match:                 password = "pass", |
| HIGH | ? | lua_test.go | 500 | Match: 		password = "pass", |
| HIGH | ? | lua_test.go | 507 | Match:         password = "pass", |
| HIGH | ? | lua_test.go | 588 | Match:         password = "pass", |
| HIGH | ? | lua_test.go | 652 | Match:         password = "pass", |
| HIGH | ? | lua_test.go | 715 | Match:         password = "pass", |
| HIGH | ? | lua_test.go | 781 | Match:         password = "pass", |
| HIGH | ? | lua_test.go | 845 | Match:         password = "pass", |
| HIGH | ? | lua_test.go | 901 | Match:         password = "pass", |
| HIGH | ? | lua_test.go | 968 | Match:         password = "pass", |
| HIGH | ? | kubernetes_test.go | 103 | Match: 			password: "pass", |
| HIGH | ? | kubernetes_test.go | 108 | Match: 			password: "htpassword", |
| HIGH | ? | kubernetes_test.go | 113 | Match: 			password: "htpasswordfile", |
| HIGH | ? | admin.pb.go | 544 | Match: 	Env       map[string]string      `protobuf:"bytes,4, |
| HIGH | ? | .goreleaser.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .devcontainer.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | accept_env.conf | 0 | File accept_env.conf has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | banner.conf | 0 | File banner.conf has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | no_penalties.conf | 0 | File no_penalties.conf has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | trusted-ca.conf | 0 | File trusted-ca.conf has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | trusted-ca.key | 0 | File trusted-ca.key has permissions -rw-rw-r-- — readable by |
| HIGH | ? | admin_test.go | 171 | Goroutine without context cancellation or done channel |
| HIGH | ? | conn_test.go | 19 | Goroutine without context cancellation or done channel |
| HIGH | ? | listener_test.go | 26 | Goroutine without context cancellation or done channel |
| HIGH | ? | cmd_test.go | 21 | Goroutine without context cancellation or done channel |
| HIGH | ? | pluginbase.go | 175 | Goroutine without context cancellation or done channel |
| HIGH | ? | grpcplugin_test.go | 30 | Goroutine without context cancellation or done channel |
| HIGH | ? | grpcplugin_test.go | 37 | Goroutine without context cancellation or done channel |
| HIGH | ? | grpcplugin_test.go | 110 | Goroutine without context cancellation or done channel |
| HIGH | ? | main_test.go | 71 | Goroutine without context cancellation or done channel |
| HIGH | ? | service_test.go | 31 | Goroutine without context cancellation or done channel |
| HIGH | ? | service_test.go | 123 | Goroutine without context cancellation or done channel |
| HIGH | ? | service_test.go | 208 | Goroutine without context cancellation or done channel |
| HIGH | ? | messagestream_test.go | 176 | Goroutine without context cancellation or done channel |
| HIGH | ? | service.go | 87 | Goroutine without context cancellation or done channel |
| HIGH | ? | service.go | 91 | Goroutine without context cancellation or done channel |
| HIGH | ? | main.go | 429 | Goroutine without context cancellation or done channel |
| HIGH | ? | main.go | 436 | Goroutine without context cancellation or done channel |
| HIGH | ? | main.go | 509 | Goroutine without context cancellation or done channel |
| HIGH | ? | main.go | 516 | Goroutine without context cancellation or done channel |
| HIGH | ? | envinject_e2e_test.go | 67 | Goroutine without context cancellation or done channel |
| HIGH | ? | envinject_e2e_test.go | 163 | Goroutine without context cancellation or done channel |
| HIGH | ? | envinject_e2e_test.go | 180 | Goroutine without context cancellation or done channel |
| HIGH | ? | envinject_e2e_test.go | 202 | Goroutine without context cancellation or done channel |
| HIGH | ? | main.go | 56 | Goroutine without context cancellation or done channel |
| HIGH | ? | daemon.go | 397 | Goroutine without context cancellation or done channel |
| HIGH | ? | daemon.go | 403 | Goroutine without context cancellation or done channel |
| HIGH | ? | main.go | 62 | Goroutine without context cancellation or done channel |
| HIGH | ? | main.go | 43 | Goroutine without context cancellation or done channel |
| HIGH | ? | lua_test.go | 261 | Goroutine without context cancellation or done channel |
| HIGH | ? | broadcaster_test.go | 89 | Goroutine without context cancellation or done channel |
| HIGH | ? | broadcaster_test.go | 109 | Goroutine without context cancellation or done channel |
| HIGH | ? | grpc.go | 641 | Goroutine without context cancellation or done channel |
| HIGH | ? | grpc.go | 646 | Goroutine without context cancellation or done channel |
| HIGH | ? | factory.go | 123 | Goroutine without context cancellation or done channel |
| HIGH | ? | ssh_server.go | 114 | Goroutine without context cancellation or done channel |
| HIGH | ? | kubectl_exec_bridge.go | 225 | Goroutine without context cancellation or done channel |
| HIGH | ? | aggregator.go | 137 | Goroutine without context cancellation or done channel |
| HIGH | ? | aggregator.go | 240 | Goroutine without context cancellation or done channel |
| HIGH | ? | dockersshd_bridge.go | 136 | Goroutine without context cancellation or done channel |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | pluginbase.go | 338 |
| H | ? | util.go | 57 |
| H | ? | skel_test.go | 172 |
| H | ? | skel.go | 76 |
| H | ? | skel.go | 106 |
| H | ? | service_test.go | 188 |
| H | ? | messagestream_test.go | 161 |
| H | ? | main.go | 137 |
| H | ? | dockersshd_bridge.go | 88 |
| H | ? | dockersshd_bridge.go | 208 |
| H | ? | dockersshd_bridge.go | 214 |
| H | ? | skel.go | 136 |
| H | ? | docker.go | 63 |
| H | ? | docker.go | 113 |
| H | ? | docker.go | 139 |
| H | ? | dockersshd_bridge_test.go | 78 |
| H | ? | dockersshd_bridge_test.go | 155 |
| H | ? | dockersshd_bridge_test.go | 158 |
| H | ? | dockersshd_bridge_test.go | 161 |
| H | ? | workingdir_test.go | 39 |
| H | ? | lua_test.go | 589 |
| H | ? | lua_test.go | 697 |
| H | ? | lua_test.go | 700 |
| H | ? | lua.go | 84 |
| H | ? | lua.go | 727 |
| H | ? | skel.go | 52 |
| H | ? | skel.go | 194 |
| H | ? | skel.go | 195 |
| H | ? | skel.go | 216 |
| H | ? | yaml.go | 125 |
| H | ? | yaml.go | 157 |
| H | ? | admin_test.go | 90 |
| H | ? | admin_test.go | 120 |
| H | ? | admin_test.go | 240 |
| H | ? | admin_test.go | 251 |
| H | ? | kubernetes_test.go | 47 |
| H | ? | kubernetes_test.go | 117 |
| H | ? | factory.go | 45 |
| H | ? | factory.go | 101 |
| H | ? | factory.go | 116 |
| H | ? | factory.go | 147 |
| H | ? | factory.go | 156 |
| H | ? | factory.go | 169 |
| H | ? | factory.go | 174 |
| H | ? | main_test.go | 178 |
| H | ? | fixed_test.go | 35 |
| H | ? | clientset_generated.go | 26 |
| H | ? | main.go | 63 |
| H | ? | main.go | 78 |
| H | ? | main.go | 379 |
| H | ? | main.go | 457 |
| H | ? | daemon_test.go | 294 |
| H | ? | asciicast.go | 67 |
| H | ? | asciicast.go | 106 |
| H | ? | asciicast.go | 154 |
| H | ? | envinject.go | 59 |
| H | ? | zz_generated.deepcopy.go | 62 |
| H | ? | zz_generated.deepcopy.go | 93 |
| H | ? | envinject_e2e_test.go | 129 |
| H | ? | kubernetes_test.go | 359 |
| H | ? | kubernetes_test.go | 362 |
| H | ? | daemon.go | 96 |
| H | ? | daemon.go | 224 |
| H | ? | daemon.go | 284 |
| H | ? | daemon.go | 375 |
| H | ? | daemon.go | 528 |
| H | ? | daemon.go | 532 |
| H | ? | skel.go | 61 |
| H | ? | skel.go | 164 |
| H | ? | skel.go | 194 |
| H | ? | skel.go | 231 |
| H | ? | skel.go | 241 |
| H | ? | skel.go | 263 |
| H | ? | skel.go | 308 |
| H | ? | hook.go | 23 |
| H | ? | kubectl_exec_bridge.go | 158 |
| H | ? | kubectl_exec_bridge.go | 168 |
| H | ? | main.go | 22 |
| H | ? | main.go | 61 |
| H | ? | server.go | 71 |
| H | ? | server.go | 113 |
| H | ? | main.go | 41 |
| H | ? | main.go | 45 |
| H | ? | main.go | 47 |
| H | ? | streamhook.go | 83 |
| H | ? | streamhook.go | 148 |
| H | ? | streamhook.go | 162 |
| H | ? | streamhook.go | 168 |
| H | ? | streamhook.go | 174 |
| H | ? | broadcaster.go | 63 |
| H | ? | broadcaster.go | 85 |
| H | ? | broadcaster.go | 104 |
| H | ? | envinject_test.go | 32 |
| H | ? | envinject_test.go | 49 |
| H | ? | envinject_test.go | 62 |
| H | ? | envinject_test.go | 90 |
| H | ? | registry_test.go | 67 |
| H | ? | main.go | 34 |
| H | ? | main.go | 153 |
| H | ? | registry.go | 77 |
| H | ? | registry.go | 94 |
| H | ? | registry.go | 111 |
| H | ? | registry.go | 124 |
| H | ? | broadcaster_test.go | 20 |
| H | ? | aggregator.go | 62 |
| H | ? | httpapi.go | 83 |
| H | ? | httpapi.go | 190 |
| H | ? | httpapi.go | 204 |
| H | ? | grpc.go | 74 |
| H | ? | grpc.go | 233 |
| H | ? | grpc.go | 247 |
| H | ? | grpc.go | 261 |
| H | ? | grpc.go | 295 |
| H | ? | grpc.go | 692 |
| H | ? | httpapi_test.go | 132 |
| H | ? | chain.go | 39 |
| H | ? | chain.go | 74 |
| H | ? | chain.go | 157 |
| H | ? | chain.go | 174 |
| H | ? | chain.go | 182 |
| H | ? | chain.go | 190 |
| H | ? | loglevel_test.go | 30 |
| H | ? | aggregator_test.go | 80 |
| H | ? | aggregator_test.go | 145 |
| H | ? | aggregator_test.go | 152 |
| H | ? | main.go | 39 |
| H | ? | main.go | 199 |
| H | ? | main.go | 230 |
| H | ? | main.go | 236 |
| H | ? | main.go | 256 |
| H | ? | main.go | 285 |
| H | ? | main.go | 290 |
| H | ? | aggregator.go | 74 |
| H | ? | aggregator.go | 96 |
| H | ? | aggregator.go | 102 |
| H | ? | aggregator.go | 103 |
| H | ? | aggregator.go | 112 |
| H | ? | aggregator.go | 113 |
| H | ? | aggregator.go | 135 |
| H | ? | aggregator.go | 165 |
| H | ? | aggregator.go | 169 |
| H | ? | aggregator.go | 170 |
| H | ? | aggregator.go | 184 |
| H | ? | aggregator.go | 198 |
| H | ? | aggregator.go | 209 |
| H | ? | aggregator.go | 227 |
| H | ? | aggregator.go | 238 |
| H | ? | aggregator.go | 250 |
| H | ? | ssh_server.go | 259 |
| H | ? | ssh_server.go | 512 |
| H | ? | ssh_server.go | 534 |
| H | ? | ssh_server.go | 547 |
| H | ? | ssh_server.go | 562 |
| H | ? | ssh_server_test.go | 38 |
| H | ? | ssh_server_test.go | 70 |
| H | ? | ssh_server_test.go | 126 |
| M | ? | main.go | 42 |
| M | ? | main.go | 53 |
| H | ? | grpcplugin_test.go | 27 |
| H | ? | grpcplugin_test.go | 40 |
| H | ? | grpcplugin_test.go | 105 |
| H | ? | clientset.go | 92 |
| H | ? | sshpiper_client.go | 61 |
| H | ? | asciicast.go | 21 |
| H | ? | clientset_generated.go | 28 |
| H | ? | grpc.go | 219 |
| H | ? | grpc.go | 673 |
| L | GS003 | build.mjs | 33 |
| L | GS003 | main.go | 72 |
| L | GS003 | main.go | 42 |
| H | ? | skel_test.go | 265 |
| H | ? | lua_test.go | 75 |
| H | ? | lua_test.go | 132 |
| H | ? | lua_test.go | 152 |
| H | ? | lua_test.go | 172 |
| H | ? | lua_test.go | 219 |
| H | ? | lua_test.go | 264 |
| H | ? | lua_test.go | 365 |
| H | ? | lua_test.go | 371 |
| H | ? | lua_test.go | 523 |
| H | ? | lua_test.go | 626 |
| H | ? | benchmark_test.go | 82 |
| H | ? | benchmark_test.go | 95 |
| H | ? | lua_test.go | 179 |
| H | ? | lua_test.go | 210 |
| H | ? | lua_test.go | 241 |
| H | ? | lua_test.go | 272 |
| H | ? | lua_test.go | 309 |
| H | ? | lua_test.go | 364 |
| H | ? | lua_test.go | 401 |
| H | ? | lua_test.go | 464 |
| H | ? | lua_test.go | 558 |
| H | ? | lua_test.go | 623 |
| H | ? | lua_test.go | 688 |
| H | ? | lua_test.go | 749 |
| H | ? | lua_test.go | 814 |
| H | ? | lua_test.go | 877 |
| H | ? | lua_test.go | 938 |
| H | ? | lua_test.go | 1006 |
| H | ? | workingdir_test.go | 87 |
| H | ? | workingdir_test.go | 209 |
| H | ? | admin_test.go | 31 |
| H | ? | admin_test.go | 35 |
| H | ? | admin_test.go | 102 |
| H | ? | admin_test.go | 140 |
| H | ? | admin_test.go | 141 |
| H | ? | admin_test.go | 279 |
| H | ? | no_penalties.conf | 1 |
| H | ? | yaml_test.go | 267 |
| H | ? | yaml_test.go | 299 |
| H | ? | yaml_test.go | 329 |
| H | ? | yaml_test.go | 360 |
| H | ? | yaml_test.go | 393 |
| H | ? | yaml_test.go | 424 |
| H | ? | yaml_test.go | 474 |
| H | ? | yaml_test.go | 507 |
| H | ? | yaml_test.go | 538 |
| H | ? | yaml_test.go | 567 |
| H | ? | docker-compose.yml | 104 |
| H | ? | docker-compose.yml | 120 |
| H | ? | grpcplugin_test.go | 25 |
| H | ? | grpcplugin_test.go | 103 |
| H | ? | main_test.go | 166 |
| H | ? | failtoban_test.go | 50 |
| H | ? | failtoban_test.go | 74 |
| H | ? | failtoban_test.go | 87 |
| H | ? | failtoban_test.go | 161 |
| H | ? | failtoban_test.go | 191 |
| H | ? | failtoban_test.go | 215 |
| H | ? | failtoban_test.go | 229 |
| H | ? | failtoban_test.go | 249 |
| H | ? | failtoban_test.go | 274 |
| H | ? | failtoban_test.go | 303 |
| H | ? | failtoban_test.go | 331 |
| H | ? | failtoban_test.go | 362 |
| H | ? | failtoban_test.go | 387 |
| H | ? | failtoban_test.go | 416 |
| H | ? | failtoban_test.go | 444 |
| H | ? | connmeta_test.go | 45 |
| H | ? | fixed_test.go | 65 |
| H | ? | fixed_test.go | 112 |
| H | ? | fixed_test.go | 144 |
| H | ? | fixed_test.go | 186 |
| H | ? | stdout_test.go | 47 |
| H | ? | docker_test.go | 44 |
| H | ? | docker_test.go | 92 |
| H | ? | docker_test.go | 134 |
| H | ? | banner_test.go | 43 |
| H | ? | banner_test.go | 101 |
| H | ? | banner_test.go | 141 |
| H | ? | main.go | 127 |
| H | ? | main.go | 276 |
| H | ? | kubectl_exec_bridge.go | 85 |
| H | ? | envinject_e2e_test.go | 30 |
| H | ? | envinject_e2e_test.go | 38 |
| H | ? | dockersshd_bridge.go | 35 |
| H | ? | server_test.go | 18 |
| H | ? | server_test.go | 22 |
| H | ? | grpc.go | 651 |
| H | ? | grpc_test.go | 51 |
| H | ? | grpc_test.go | 58 |
| H | ? | grpc_test.go | 64 |
| H | ? | grpc_test.go | 76 |
| H | ? | grpc_test.go | 82 |
| H | ? | grpc_test.go | 94 |
| H | ? | grpc_test.go | 110 |
| H | ? | grpc_test.go | 113 |
| H | ? | grpc_test.go | 130 |
| H | ? | grpc_test.go | 145 |
| H | ? | grpc_test.go | 162 |
| H | ? | ssh_server_test.go | 140 |
| H | ? | ssh_server_test.go | 196 |
| H | ? | ssh_server_test.go | 208 |
| H | ? | aggregator_test.go | 39 |
| H | ? | main.go | 54 |
| H | ? | httpapi_test.go | 44 |
| H | ? | index.html | 58 |
| C | ? | e2eentry.sh | 85 |
| C | ? | e2eentry.sh | 86 |
| C | ? | daemon.go | 326 |
| H | ? | plugin.pb.go | 81 |
| H | ? | plugin.pb.go | 172 |
| H | ? | plugin.pb.go | 547 |
| H | ? | plugin.pb.go | 591 |
| H | ? | lua_test.go | 26 |
| H | ? | lua_test.go | 71 |
| H | ? | lua_test.go | 90 |
| H | ? | lua_test.go | 500 |
| H | ? | lua_test.go | 507 |
| H | ? | lua_test.go | 588 |
| H | ? | lua_test.go | 652 |
| H | ? | lua_test.go | 715 |
| H | ? | lua_test.go | 781 |
| H | ? | lua_test.go | 845 |
| H | ? | lua_test.go | 901 |
| H | ? | lua_test.go | 968 |
| H | ? | kubernetes_test.go | 103 |
| H | ? | kubernetes_test.go | 108 |
| H | ? | kubernetes_test.go | 113 |
| H | ? | admin.pb.go | 544 |
| M | ? | main.go | 8 |
| H | ? | .goreleaser.yaml | 0 |
| H | ? | .devcontainer.json | 0 |
| H | GS002 | accept_env.conf | 0 |
| H | GS002 | banner.conf | 0 |
| H | GS002 | no_penalties.conf | 0 |
| H | GS002 | trusted-ca.conf | 0 |
| H | GS002 | trusted-ca.key | 0 |
| s | GS009 |  | 0 |
| M | GS014 | trusted-ca.key | 0 |
| H | ? | admin_test.go | 171 |
| H | ? | conn_test.go | 19 |
| H | ? | listener_test.go | 26 |
| H | ? | cmd_test.go | 21 |
| H | ? | pluginbase.go | 175 |
| H | ? | grpcplugin_test.go | 30 |
| H | ? | grpcplugin_test.go | 37 |
| H | ? | grpcplugin_test.go | 110 |
| H | ? | main_test.go | 71 |
| H | ? | service_test.go | 31 |
| H | ? | service_test.go | 123 |
| H | ? | service_test.go | 208 |
| H | ? | messagestream_test.go | 176 |
| H | ? | service.go | 87 |
| H | ? | service.go | 91 |
| H | ? | main.go | 429 |
| H | ? | main.go | 436 |
| H | ? | main.go | 509 |
| H | ? | main.go | 516 |
| H | ? | envinject_e2e_test.go | 67 |
| H | ? | envinject_e2e_test.go | 163 |
| H | ? | envinject_e2e_test.go | 180 |
| H | ? | envinject_e2e_test.go | 202 |
| H | ? | main.go | 56 |
| H | ? | daemon.go | 397 |
| H | ? | daemon.go | 403 |
| H | ? | main.go | 62 |
| H | ? | main.go | 43 |
| H | ? | lua_test.go | 261 |
| H | ? | broadcaster_test.go | 89 |
| H | ? | broadcaster_test.go | 109 |
| H | ? | grpc.go | 641 |
| H | ? | grpc.go | 646 |
| H | ? | factory.go | 123 |
| H | ? | ssh_server.go | 114 |
| H | ? | kubectl_exec_bridge.go | 225 |
| H | ? | aggregator.go | 137 |
| H | ? | aggregator.go | 240 |
| H | ? | dockersshd_bridge.go | 136 |
| M | ? | messagestream.go | 28 |
| M | ? | messagestream.go | 31 |
| M | ? | envinject_e2e_test.go | 155 |
| M | ? | lua.go | 29 |
| M | ? | lua.go | 30 |
| M | ? | lua.go | 31 |
| M | ? | factory.go | 26 |
| M | ? | factory.go | 36 |
| M | ? | streamhook.go | 33 |
| M | ? | broadcaster.go | 36 |
| M | ? | registry.go | 50 |
| M | ? | broadcaster_test.go | 107 |
| M | ? | aggregator.go | 22 |
| M | ? | kubernetes.go | 25 |
| M | ? | ssh_server.go | 199 |
| M | ? | ssh_server.go | 465 |
| M | ? | client.go | 142 |
| M | ? | dockersshd_bridge.go | 138 |
| M | ? | docker.go | 31 |
| M | ? | aggregator.go | 44 |
| M | ? | aggregator.go | 129 |
| M | ? | aggregator.go | 130 |
| M | ? | aggregator.go | 233 |
| M | ? | aggregator.go | 234 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:21:58.632441*